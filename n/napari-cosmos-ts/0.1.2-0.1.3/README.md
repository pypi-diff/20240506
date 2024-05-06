# Comparing `tmp/napari_cosmos_ts-0.1.2.tar.gz` & `tmp/napari_cosmos_ts-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari_cosmos_ts-0.1.2.tar", last modified: Fri Apr 12 14:05:26 2024, max compression
+gzip compressed data, was "napari_cosmos_ts-0.1.3.tar", last modified: Mon May  6 21:03:44 2024, max compression
```

## Comparing `napari_cosmos_ts-0.1.2.tar` & `napari_cosmos_ts-0.1.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1077 2024-04-04 20:40:34.143863 napari_cosmos_ts-0.1.2/LICENSE
--rw-r--r--   0        0        0     1658 2024-04-11 15:56:00.131898 napari_cosmos_ts-0.1.2/README.md
--rw-r--r--   0        0        0     1177 2024-04-12 14:05:26.584771 napari_cosmos_ts-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-09 15:49:27.422300 napari_cosmos_ts-0.1.2/src/napari_cosmos_ts/__init__.py
--rw-r--r--   0        0        0    80704 2024-04-12 14:00:03.448745 napari_cosmos_ts-0.1.2/src/napari_cosmos_ts/main_widget.py
--rw-r--r--   0        0        0      311 2024-04-11 15:00:04.753800 napari_cosmos_ts-0.1.2/src/napari_cosmos_ts/napari.yaml
--rw-r--r--   0        0        0        0 2024-04-09 15:49:27.423781 napari_cosmos_ts-0.1.2/tests/__init__.py
--rw-r--r--   0        0        0     2557 1970-01-01 00:00:00.000000 napari_cosmos_ts-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-04-04 20:40:34.143863 napari_cosmos_ts-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1852 2024-04-22 14:05:21.046015 napari_cosmos_ts-0.1.3/README.md
+-rw-r--r--   0        0        0     1177 2024-05-06 21:03:44.087463 napari_cosmos_ts-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-09 15:49:27.422300 napari_cosmos_ts-0.1.3/src/napari_cosmos_ts/__init__.py
+-rw-r--r--   0        0        0    87724 2024-05-06 20:49:23.297635 napari_cosmos_ts-0.1.3/src/napari_cosmos_ts/main_widget.py
+-rw-r--r--   0        0        0      311 2024-04-11 15:00:04.753800 napari_cosmos_ts-0.1.3/src/napari_cosmos_ts/napari.yaml
+-rw-r--r--   0        0        0        0 2024-04-09 15:49:27.423781 napari_cosmos_ts-0.1.3/tests/__init__.py
+-rw-r--r--   0        0        0     2751 1970-01-01 00:00:00.000000 napari_cosmos_ts-0.1.3/PKG-INFO
```

### Comparing `napari_cosmos_ts-0.1.2/LICENSE` & `napari_cosmos_ts-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `napari_cosmos_ts-0.1.2/README.md` & `napari_cosmos_ts-0.1.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -11,18 +11,25 @@
 ```shell
 conda activate napari-env
 ```
 4. Install `napari` and `napari-cosmos-ts` into your virtual environment. In a command shell or terminal *where you have activated your virtual environment* run the following command:
 ```shell
 pip install "napari[all]" napari-cosmos-ts
 ```
+Or for the latest version of `napari-cosmos-ts`:
+```shell
+pip install "napari[all]" napari-cosmos-ts@git+https://github.com/marcel-goldschen-ohm/napari-cosmos-ts
+```
 
 # Run
 1. Activate your virtual environment (see [Install](#install), replace napari-env with the name of your environment). In a command shell or terminal run the following command:
 ```shell
 conda activate napari-env
 ```
 2. Launch the `napari` viewer. In a command shell or terminal *where you have activated your virtual environment* run the following command:
 ```shell
 napari
 ```
 3. Launch the `napari-cosmos-ts` plugin. From the napari viewer `Plugins menu`, select `Colocalization Single-Molecule Time Series (napari-cosmos-ts)`. This should bring up a docked widget within the viewer. **Now you are good to go!**
+
+# User Guide
+:construction:
```

### Comparing `napari_cosmos_ts-0.1.2/pyproject.toml` & `napari_cosmos_ts-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: MIT License",
     "Framework :: napari",
     "Programming Language :: Python :: 3 :: Only",
 ]
-version = "0.1.2"
+version = "0.1.3"
 
 [project.license]
 text = "MIT"
 
 [project.entry-points."napari.manifest"]
 napari-cosmos-ts = "napari_cosmos_ts:napari.yaml"
```

### Comparing `napari_cosmos_ts-0.1.2/src/napari_cosmos_ts/main_widget.py` & `napari_cosmos_ts-0.1.3/src/napari_cosmos_ts/main_widget.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,14 +53,15 @@
         
         # session dict
         session = {}
         session['date'] = self._date_edit.text() + " "
         session['ID'] = self._id_edit.text() + " "
         session['users'] = self._users_edit.text() + " "
         session['notes'] = self._notes_edit.toPlainText() + " "
+        session['default_point_size'] = self._default_point_size_spinbox.value()
         
         # layer dicts
         session['layers'] = []
         for layer in self.viewer.layers:
             layer_data = {}
             layer_data['name'] = layer.name
             layer_data['affine'] = layer.affine.affine_matrix
@@ -138,14 +139,16 @@
                 self._date_edit.setText(str(value).strip())
             elif key == "ID":
                 self._id_edit.setText(str(value).strip())
             elif key == "users":
                 self._users_edit.setText(str(value).strip())
             elif key == "notes":
                 self._notes_edit.setPlainText(str(value).strip())
+            elif key == "default_point_size":
+                self._default_point_size_spinbox.setValue(session['default_point_size'])
             elif key == "layers":
                 for layer_data in value:
                     layer = None
                     
                     if layer_data['type'] == 'image':
                         abspath = None
                         if 'relpath' in layer_data:
@@ -506,15 +509,15 @@
         n_points = len(points)
 
         new_layer = self.viewer.add_points(
             points,
             name = layer.name + " (peaks)",
             affine = layer.affine.affine_matrix[-3:,-3:],
             symbol = "disc",
-            size = [self._point_size_spinbox.value()] * n_points,
+            size = [self._default_point_size_spinbox.value()] * n_points,
             face_color = [[1, 1, 0, 0.1]] * n_points,
             edge_color = [[1, 1, 0, 1]] * n_points,
             opacity = 1,
             blending = "translucent_no_depth",
         )
         return new_layer
 
@@ -549,23 +552,23 @@
 
         # colocalized points layer
         n_points = len(colocalized)
         new_layer = self.viewer.add_points(
             colocalized,
             name = "colocalized",
             symbol = "disc",
-            size = [self._point_size_spinbox.value()] * n_points,
+            size = [self._default_point_size_spinbox.value()] * n_points,
             face_color = [[1, 0, 1, 0.1]] * n_points,
             edge_color = [[1, 0, 1, 1]] * n_points,
             opacity = 1,
             blending = "translucent_no_depth",
         )
         return new_layer
     
-    def set_projection_point(self, worldpt2d: np.ndarray | None):
+    def set_projection_point(self, worldpt2d: np.ndarray | None, point_size: int | float = None):
         """ Set the world position for the currently visible point projections.
 
         This will update the point projection plots for all image stack layers.
         """
         if worldpt2d is None:
             # clear selected projection point overlay
             if self._selected_point_layer is not None:
@@ -580,50 +583,69 @@
             # update point projections tab
             self._projection_point_world_label.setText("")
             self._tag_edit.setText("")
             
             return
         
         worldpt2d = np.array(worldpt2d).reshape([1, 2])
+
+        if point_size is None:
+            point_size = self._default_point_size_spinbox.value()
         
         # update selected projection point overlay
         if self._selected_point_layer is None:
             self._selected_point_layer = self.viewer.add_points(
                 worldpt2d,
                 name = "selected point",
                 symbol = "disc",
-                size = [self._point_size_spinbox.value()],
+                size = [point_size],
                 face_color = [[0, 1, 1, 0.1]],
                 edge_color = [[0, 1, 1, 1]],
                 opacity = 1,
                 blending = "translucent_no_depth",
             )
             self._selected_point_layer.metadata['is_selected_point_layer'] = True
             # because self._selected_point_layer is not yet defined during layer insertion
             self._update_layer_selection_comboboxes(self._selected_point_layer)
         else:
             self._selected_point_layer.data = worldpt2d
+            self._selected_point_layer.size = [point_size]
         
         # update point projections tab
         row, col = np.round(worldpt2d).astype(int).flatten()
         self._projection_point_world_label.setText(f"[{row}, {col}]")
         self._tag_edit.setText("")
         
         # project selected point for all imagestack layers
-        point_size = int(np.round(self._selected_point_layer.size[0]))
-        point_mask = np.ones([point_size, point_size])
+        # use circular mask for point projection
+        pixel_size = int(np.round(self._selected_point_layer.size[0]))
+        point_mask = make_point_mask(pixel_size, type='circle')
         for layer, metadata in zip(self.viewer.layers, self._layer_metadata):
             if isinstance(layer, Image) and layer.data.ndim == 3:
                 if 'point_projection_data' in metadata:
                     # selected point in layer
                     layerpt2d = self._transform_points2d_from_world_to_layer(worldpt2d, layer)
                     # project point
-                    point_projection = project_image_point(layer.data, layerpt2d, point_mask)
+                    xdata = None  # assumed integer frames
+                    ydata = project_image_point(layer.data, layerpt2d, point_mask)
+                    # sum frames?
+                    if 'projection-sum-frames' in metadata:
+                        nframes = metadata['projection-sum-frames']
+                        if nframes > 1:
+                            xdata = np.arange(0, len(ydata), nframes)
+                            tmp_ydata = np.zeros(xdata.shape)
+                            for i in range(nframes):
+                                tmp = ydata[i::nframes]
+                                tmp_ydata[:len(tmp)] += tmp
+                            ydata = tmp_ydata
                     # update plot
-                    metadata['point_projection_data'].setData(point_projection)
+                    if xdata is None:
+                        metadata['point_projection_data'].setData(ydata)
+                    else:
+                        metadata['point_projection_data'].setData(xdata, ydata)
     
     def select_projection_point(self, layer: Points = None, point_index: int = None, ignore_tag_filter: bool = False):
         """ Select an existing point to use as the position for the currently visible point projections.
 
         The selected point will be used for projection in all image stack layers.
         """
         # add guard because blockSignals() does not work for QSpinBox.valueChanged
@@ -695,15 +717,16 @@
                                     break
                     if found_point:
                         self._projection_point_index_spinbox.setValue(point_index)
 
             # project point
             layerpt2d = layer.data[point_index,-2:]
             worldpt2d = self._transform_points2d_from_layer_to_world(layerpt2d, layer)
-            self.set_projection_point(worldpt2d)
+            point_size = layer.size[point_index]
+            self.set_projection_point(worldpt2d, point_size)
 
             # show point tags
             try:
                 tags: str = layer.features['tags'][point_index]
             except (KeyError, IndexError):
                 tags = ""
             self._tag_edit.setText(tags)
@@ -713,14 +736,32 @@
 
         # keep track of currently selected point
         self._selected_point_index = point_index
         
         # remove guard
         self._select_projection_point_in_progress = False
     
+    def update_point_projections(self):
+        is_index_selected = self._projection_point_index_spinbox.text().strip() != ''
+        if is_index_selected:
+            index = self._projection_point_index_spinbox.value()
+            layer_name = self._projection_points_layer_combobox.currentText()
+            try:
+                layer = self.viewer.layers[layer_name]
+                self.select_projection_point(layer, index, ignore_tag_filter=True)
+                return
+            except KeyError:
+                pass
+        
+        # no index selected, check for selected point layer
+        if self._selected_point_layer is not None:
+            worldpt2d = self._selected_point_layer.data
+            self.set_projection_point(worldpt2d)
+            return
+    
     def set_point_tags(self, layer: Points = None, point_index: int = None, tags: str = None):
         """ Set tags for a point.
 
         The tags string will be stored in the 'tags' feature column of the layer.
         """
         if layer is None:
             layer_name = self._projection_points_layer_combobox.currentText()
@@ -961,20 +1002,23 @@
             if 'point_projection_vline' in metadata:
                 vline = metadata['point_projection_vline']
                 vline.setValue(frame)
 
     def _on_mouse_clicked_or_dragged(self, viewer: Viewer, event: Event):
         """ Callback for mouse press/drag/release events.
         """
+        from qtpy.QtCore import Qt
+
         if viewer.layers.selection.active.mode != "pan_zoom":
             return
         
         # mouse press event
+        # only process left-click events
         # ignore initial mouse press event (we'll use the mouse release event instead)
-        if event.type == 'mouse_press':
+        if (event.type == 'mouse_press') and (event._button == Qt.MouseButton.LeftButton):
             yield
         else:
             return
 
         # mouse move event
         # if mouse dragged (beyond a tiny bit), ignore subsequent mouse release event
         # i.e., ignore click when dragging
@@ -1131,15 +1175,15 @@
     def _setup_file_tab(self, title: str = "File"):
         """ File UI.
 
         Includes session import/export.
         """
         from qtpy.QtWidgets import QHBoxLayout, QVBoxLayout, QPushButton, QWidget, QLabel
 
-        msg = QLabel("!!! Session stores the relative path to each image stack file, NOT the data itself. It is up to you to maintain this file structure. !!!")
+        msg = QLabel("!!! Session stores the relative path to each image stack file, NOT the data itself. It is up to you to maintain this file structure.\nSession .mat files can be accessed in MATLAB.")
         msg.setWordWrap(True)
 
         self._open_session_button = QPushButton("Open .mat session file")
         self._open_session_button.pressed.connect(self.import_session)
 
         self._save_session_button = QPushButton("Save session as .mat file")
         self._save_session_button.pressed.connect(self.export_session)
@@ -1199,62 +1243,62 @@
         self._tophat_filter_button = QPushButton("Tophat Filter")
         self._tophat_filter_button.pressed.connect(lambda: self._apply_to_selected_layers(self.filter_image_layer, filter_type="tophat"))
 
         self._tophat_filter_disk_radius_spinbox = QDoubleSpinBox()
         self._tophat_filter_disk_radius_spinbox.setValue(3)
 
         tab = QTabWidget()
-        for tab_title in ["Split", "Slice", "Project", "Filter"]:
+        for tab_title in ["Split/Slice", "Project", "Filter"]:
             msg = QLabel("Operations are applied to all selected image layers.\nResults are returned in new layers.")
             msg.setWordWrap(True)
 
             inner = QVBoxLayout()
             inner.setContentsMargins(0, 0, 0, 0)
             inner.setSpacing(5)
             inner.addWidget(msg)
-            if tab_title == "Split":
+            if tab_title == "Split/Slice":
                 group = QGroupBox()
                 form = QFormLayout(group)
                 form.setContentsMargins(5, 5, 5, 5)
                 form.setSpacing(5)
                 form.addRow(self._split_image_button)
-                form.addRow("regions", self._split_image_regions_combobox)
+                form.addRow("Regions", self._split_image_regions_combobox)
                 inner.addWidget(group)
-            elif tab_title == "Slice":
+
                 group = QGroupBox()
                 form = QFormLayout(group)
                 form.setContentsMargins(5, 5, 5, 5)
                 form.setSpacing(5)
                 form.setFieldGrowthPolicy(QFormLayout.AllNonFixedFieldsGrow)
                 form.addRow(self._slice_image_button)
-                form.addRow("slice", self._slice_image_edit)
+                form.addRow("Slice", self._slice_image_edit)
                 inner.addWidget(group)
             elif tab_title == "Project":
                 group = QGroupBox()
                 form = QFormLayout(group)
                 form.setContentsMargins(5, 5, 5, 5)
                 form.setSpacing(5)
                 form.addRow(self._project_image_button)
-                form.addRow("projection", self._project_image_operation_combobox)
+                form.addRow("Projection", self._project_image_operation_combobox)
                 inner.addWidget(group)
             elif tab_title == "Filter":
                 group = QGroupBox()
                 form = QFormLayout(group)
                 form.setContentsMargins(5, 5, 5, 5)
                 form.setSpacing(5)
                 form.addRow(self._gaussian_filter_button)
-                form.addRow("sigma", self._gaussian_filter_sigma_spinbox)
+                form.addRow("Sigma", self._gaussian_filter_sigma_spinbox)
                 inner.addWidget(group)
                 
                 group = QGroupBox()
                 form = QFormLayout(group)
                 form.setContentsMargins(5, 5, 5, 5)
                 form.setSpacing(5)
                 form.addRow(self._tophat_filter_button)
-                form.addRow("disk radius", self._tophat_filter_disk_radius_spinbox)
+                form.addRow("Disk radius", self._tophat_filter_disk_radius_spinbox)
                 inner.addWidget(group)
             inner.addStretch()
 
             outer = QHBoxLayout()
             outer.setContentsMargins(5, 5, 5, 5)
             outer.setSpacing(5)
             outer.addLayout(inner)
@@ -1270,45 +1314,51 @@
         """ Points UI.
 
         Includes point settings, colocalization, and point projection.
         """
         from qtpy.QtCore import Qt
         from qtpy.QtWidgets import QHBoxLayout, QVBoxLayout, QWidget, QFormLayout, QGroupBox, QPushButton, QSpinBox, QDoubleSpinBox, QComboBox, QTabWidget, QGridLayout, QLabel, QCheckBox, QLineEdit
 
-        self._point_size_spinbox = QDoubleSpinBox()
-        self._point_size_spinbox.setValue(8)
+        self._default_point_size_spinbox = QDoubleSpinBox()
+        self._default_point_size_spinbox.setValue(8)
+
+        self._default_point_mask_grid = QGridLayout()
+        self._default_point_mask_grid.setContentsMargins(5, 5, 5, 5)
+        self._default_point_mask_grid.setSpacing(2)
+        self._update_default_point_mask_grid()
+        self._default_point_size_spinbox.valueChanged.connect(self._update_default_point_mask_grid)
 
         self._find_peaks_button = QPushButton("Find peaks in all selected image layers")
         self._find_peaks_button.pressed.connect(lambda: self._apply_to_selected_layers(self.find_image_peaks))
 
         self._min_peak_height_spinbox = QDoubleSpinBox()
         self._min_peak_height_spinbox.setMinimum(0)
         self._min_peak_height_spinbox.setMaximum(65000)
         self._min_peak_height_spinbox.setValue(10)
 
         self._min_peak_separation_spinbox = QDoubleSpinBox()
         self._min_peak_separation_spinbox.setMinimum(1)
         self._min_peak_separation_spinbox.setMaximum(65000)
-        self._min_peak_separation_spinbox.setValue(self._point_size_spinbox.value())
+        self._min_peak_separation_spinbox.setValue(self._default_point_size_spinbox.value())
 
         self._find_colocalized_points_button = QPushButton("Find colocalized points")
         self._find_colocalized_points_button.pressed.connect(self.find_colocalized_points)
 
         self._coloc_layer_combobox = QComboBox()
         self._coloc_layer_combobox.currentTextChanged.connect(lambda text: self._update_points_colocalization_plot())
         
         self._coloc_neighbors_layer_combobox = QComboBox()
         self._coloc_neighbors_layer_combobox.currentTextChanged.connect(lambda text: self._update_points_colocalization_plot())
 
         self._coloc_nearest_neighbor_cutoff_spinbox = QDoubleSpinBox()
-        self._coloc_nearest_neighbor_cutoff_spinbox.setValue(self._point_size_spinbox.value() / 2)
+        self._coloc_nearest_neighbor_cutoff_spinbox.setValue(self._default_point_size_spinbox.value() / 2)
 
         self._coloc_hist_binwidth_spinbox = QDoubleSpinBox()
         self._coloc_hist_binwidth_spinbox.setMinimum(1)
-        self._coloc_hist_binwidth_spinbox.setValue(self._point_size_spinbox.value() / 2)
+        self._coloc_hist_binwidth_spinbox.setValue(self._default_point_size_spinbox.value() / 2)
         self._coloc_hist_binwidth_spinbox.valueChanged.connect(lambda value: self._update_points_colocalization_plot())
 
         self._coloc_plot = self._new_plot()
         self._coloc_plot.setLabels(left="Counts", bottom="Nearest Neighbor Distance")
         legend = pg.LegendItem()
         legend.setParentItem(self._coloc_plot.getPlotItem())
         legend.anchor((1,0), (1,0))
@@ -1337,47 +1387,69 @@
 
         self._tag_filter_checkbox = QCheckBox("Tag filter")
         self._tag_filter_checkbox.stateChanged.connect(lambda state: self._update_tag_filter())
 
         self._tag_filter_edit = QLineEdit()
         self._tag_filter_edit.editingFinished.connect(self._update_tag_filter)
 
+        self._projection_settings_button = QPushButton("Settings")
+        self._projection_settings_button.pressed.connect(self._edit_projection_settings)
+
         tab = QTabWidget()
-        for tab_title in ["Size", "Find", "Colocalize", "Projection"]:
+        for tab_title in ["Point", "Find", "Colocalize", "Projection"]:
             inner = QVBoxLayout()
             inner.setContentsMargins(0, 0, 0, 0)
             inner.setSpacing(5)
-            if tab_title == "Size":
+            if tab_title == "Point":
+                msg = QLabel("Point projections use a circular mask centered on the point with pixel diameter equal to the selected point's size. For projecting an arbitrary position, the default size below will be used.")
+                msg.setWordWrap(True)
+
                 group = QGroupBox()
                 form = QFormLayout(group)
                 form.setContentsMargins(5, 5, 5, 5)
                 form.setSpacing(5)
-                form.addRow("Default point size", self._point_size_spinbox)
+                form.addRow(msg)
+                form.addRow("Default point size", self._default_point_size_spinbox)
                 inner.addWidget(group)
+
+                inner.addSpacing(10)
+                inner.addWidget(QLabel("Default point projection mask"))
+                inner.addLayout(self._default_point_mask_grid)
             elif tab_title == "Find":
                 group = QGroupBox()
                 form = QFormLayout(group)
                 form.setContentsMargins(5, 5, 5, 5)
                 form.setSpacing(5)
                 form.addRow(self._find_peaks_button)
                 form.addRow("Min peak height", self._min_peak_height_spinbox)
                 form.addRow("Min peak separation", self._min_peak_separation_spinbox)
                 inner.addWidget(group)
             elif tab_title == "Colocalize":
+                grid = QGridLayout()
+                grid.setContentsMargins(0, 0, 0, 0)
+                grid.setSpacing(0)
+
                 group = QGroupBox()
                 form = QFormLayout(group)
                 form.setContentsMargins(5, 5, 5, 5)
                 form.setSpacing(5)
                 form.addRow(self._find_colocalized_points_button)
                 form.addRow("Points layer", self._coloc_layer_combobox)
                 form.addRow("Neighbors points layer", self._coloc_neighbors_layer_combobox)
                 form.addRow("Nearest neighbor cutoff", self._coloc_nearest_neighbor_cutoff_spinbox)
+                grid.addWidget(group, 0, 0)
+
+                form = QFormLayout()
+                form.setContentsMargins(5, 5, 5, 5)
+                form.setSpacing(5)
                 form.addRow("Histogram bin width", self._coloc_hist_binwidth_spinbox)
-                form.addRow(self._coloc_plot)
-                inner.addWidget(group)
+                grid.addLayout(form, 1, 0)
+                grid.addWidget(self._coloc_plot, 2, 0, 1, 2)
+                
+                inner.addLayout(grid)
             elif tab_title == "Projection":
                 grid = QGridLayout()
                 grid.setContentsMargins(0, 0, 0, 0)
                 grid.setSpacing(5)
                 layer_label = QLabel("Points layer")
                 layer_label.setAlignment(Qt.AlignmentFlag.AlignRight | Qt.AlignmentFlag.AlignVCenter)
                 index_label = QLabel("Point index")
@@ -1390,14 +1462,15 @@
                 grid.addWidget(self._tag_filter_checkbox, 0, 3)
                 grid.addWidget(self._tag_filter_edit, 0, 4)
                 grid.addWidget(index_label, 1, 0)
                 grid.addWidget(self._projection_point_index_spinbox, 1, 1)
                 grid.addWidget(self._projection_point_world_label, 1, 2)
                 grid.addWidget(tag_label, 1, 3)
                 grid.addWidget(self._tag_edit, 1, 4)
+                grid.addWidget(self._projection_settings_button, 1, 5)
                 inner.addLayout(grid)
                 inner.addLayout(self._point_projection_plots_layout)
             
             if tab_title == "Projection":
                 tab2 = QWidget()
                 tab2.setLayout(inner)
                 tab.addTab(tab2, tab_title)
@@ -1445,17 +1518,17 @@
 
         layer_registration_group = QGroupBox()
         form = QFormLayout(layer_registration_group)
         form.setFieldGrowthPolicy(QFormLayout.AllNonFixedFieldsGrow)
         form.setContentsMargins(5, 5, 5, 5)
         form.setSpacing(5)
         form.addRow(self._register_layers_button)
-        form.addRow("fixed Layer", self._fixed_layer_combobox)
-        form.addRow("moving Layer", self._moving_layer_combobox)
-        form.addRow("transform", self._layer_transform_type_combobox)
+        form.addRow("Fixed Layer", self._fixed_layer_combobox)
+        form.addRow("Moving Layer", self._moving_layer_combobox)
+        form.addRow("Transform", self._layer_transform_type_combobox)
 
         inner = QVBoxLayout()
         inner.setContentsMargins(0, 0, 0, 0)
         inner.setSpacing(5)
         inner.addWidget(msg)
         inner.addWidget(layer_registration_group)
         inner.addWidget(self._copy_layer_transform_button)
@@ -1520,14 +1593,31 @@
         if items:
             combobox.addItems(items)
             if current_text in items:
                 combobox.setCurrentText(current_text)
             elif 0 <= current_index < len(items):
                 combobox.setCurrentIndex(current_index)
     
+    def _update_default_point_mask_grid(self):
+        from qtpy.QtCore import Qt
+        from qtpy.QtWidgets import QLabel
+
+        clear_layout(self._default_point_mask_grid)
+        point_size = self._default_point_size_spinbox.value()
+        point_mask = make_point_mask(point_size, type='circle')
+        for i, row in enumerate(point_mask):
+            for j, value in enumerate(row):
+                label = QLabel(str(float(value)))
+                bg = int(255 * value)
+                fg = 0 if bg >= 128 else 255
+                label.setStyleSheet(f"QLabel {{ background-color : rgb({bg}, {bg}, {bg}); color : rgb({fg}, {fg}, {fg}); }}")
+                label.setAlignment(Qt.AlignmentFlag.AlignCenter | Qt.AlignmentFlag.AlignVCenter)
+                label.setFixedSize(30, 30)
+                self._default_point_mask_grid.addWidget(label, i, j)
+    
     def _update_points_colocalization_plot(self, layer: Points = None, neighbors_layer: Points = None, nearest_neighbor_cutoff: float = None, binwidth: float = None):
         """ Update within layer and between layers nearest neighbor histograms for selected points layers.
         """
         from scipy.spatial import distance
 
         if layer is None:
             layer_name = self._coloc_layer_combobox.currentText()
@@ -1585,14 +1675,66 @@
         else:
             self._within_layers_nearest_neighbors_histogram.setData([0, 0], [0])
             self._between_layers_nearest_neighbors_histogram.setData([0, 0], [0])
 
     def _update_tag_filter(self):
         if self._tag_filter_checkbox.isChecked():
             self.select_projection_point()
+    
+    def _edit_projection_settings(self):
+        from qtpy.QtWidgets import QDialog, QVBoxLayout, QGroupBox, QFormLayout, QDialogButtonBox, QSpinBox
+
+        dlg = QDialog(self)
+        dlg.setWindowTitle("Point Projection Settings")
+        vbox = QVBoxLayout(dlg)
+
+        group = QGroupBox("Sum Frames")
+        form = QFormLayout(group)
+        sum_frames_spinboxes = {}
+        for layer, metadata in zip(reversed(self.viewer.layers), reversed(self._layer_metadata)):
+            if isinstance(layer, Image) and layer.data.ndim == 3:
+                spinbox = QSpinBox()
+                spinbox.setMinimum(1)
+                spinbox.setMaximum(layer.data.shape[-3])
+                if 'projection-sum-frames' in metadata:
+                    spinbox.setValue(metadata['projection-sum-frames'])
+                form.addRow(layer.name, spinbox)
+                sum_frames_spinboxes[layer.name] = spinbox
+        vbox.addWidget(group)
+
+        buttons = QDialogButtonBox(QDialogButtonBox.StandardButton.Ok | QDialogButtonBox.StandardButton.Cancel)
+        buttons.accepted.connect(dlg.accept)
+        buttons.rejected.connect(dlg.reject)
+        vbox.addWidget(buttons)
+
+        if dlg.exec() != QDialog.Accepted:
+            return
+        
+        for layer, metadata in zip(reversed(self.viewer.layers), reversed(self._layer_metadata)):
+            if isinstance(layer, Image) and layer.data.ndim == 3:
+                spinbox = sum_frames_spinboxes[layer.name]
+                if spinbox.value() != 1:
+                    metadata['projection-sum-frames'] = spinbox.value()
+                elif 'projection-sum-frames' in metadata:
+                    del metadata['projection-sum-frames']
+        
+        self.update_point_projections()
+
+
+def clear_layout(layout: 'qtpy.QtWidgets.QLayout'):
+    from qtpy.QtWidgets import QLayout
+
+    for i in reversed(range(layout.count())):
+        item = layout.itemAt(i)
+        if isinstance(item, QLayout):
+            clear_layout(item)
+        elif item.widget():
+            item.widget().setParent(None)
+        else:
+            layout.removeItem(item)
 
 
 def slice_from_str(slice_str: str) -> tuple[slice]:
     """ Convert string to slice.
     """
     if slice_str.strip() == "":
         return (slice(None),)
@@ -1773,14 +1915,26 @@
     rows = rows[i].reshape([-1,1])
     cols = cols[j].reshape([1,-1])
     mask = point_mask2d[i.reshape([-1,1]),j.reshape([1,-1])]
     mask = mask.reshape((1,) * (image.ndim - 2) + mask.shape)
     return np.squeeze(np.mean(image[...,rows,cols] * mask, axis=(-2, -1)))
 
 
+def make_point_mask(size: int | float, type: str = 'circle'):
+    if type == 'circle':
+        radius = size / 2
+        max_pixel_offset = (size - 1) / 2
+        pixel_offsets = np.arange(-max_pixel_offset, max_pixel_offset + 1, dtype=float)
+        mask = (pixel_offsets.reshape([-1,1])**2 + pixel_offsets.reshape([1,-1])**2) <= radius**2
+        return mask
+    
+    if type == 'square':
+        return np.ones((size, size), dtype=bool)
+
+
 if __name__ == "__main__":
     """ This is mostly for debugging.
     
     Typically, the plugin is run from the plugin menu in the napari viewer.
     """
     import napari
```

### Comparing `napari_cosmos_ts-0.1.2/PKG-INFO` & `napari_cosmos_ts-0.1.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-cosmos-ts
-Version: 0.1.2
+Version: 0.1.3
 Summary: napari plugin for colocalization single-molecule spectroscopy (CoSMoS) time series (TS) analysis
 Home-page: https://github.com/marcel-goldschen-ohm/napari-cosmos-ts
 Author-Email: Marcel Goldschen-Ohm <goldschen-ohm@utexas.edu>
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
@@ -32,18 +32,25 @@
 ```shell
 conda activate napari-env
 ```
 4. Install `napari` and `napari-cosmos-ts` into your virtual environment. In a command shell or terminal *where you have activated your virtual environment* run the following command:
 ```shell
 pip install "napari[all]" napari-cosmos-ts
 ```
+Or for the latest version of `napari-cosmos-ts`:
+```shell
+pip install "napari[all]" napari-cosmos-ts@git+https://github.com/marcel-goldschen-ohm/napari-cosmos-ts
+```
 
 # Run
 1. Activate your virtual environment (see [Install](#install), replace napari-env with the name of your environment). In a command shell or terminal run the following command:
 ```shell
 conda activate napari-env
 ```
 2. Launch the `napari` viewer. In a command shell or terminal *where you have activated your virtual environment* run the following command:
 ```shell
 napari
 ```
 3. Launch the `napari-cosmos-ts` plugin. From the napari viewer `Plugins menu`, select `Colocalization Single-Molecule Time Series (napari-cosmos-ts)`. This should bring up a docked widget within the viewer. **Now you are good to go!**
+
+# User Guide
+:construction:
```

